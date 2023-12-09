<html>

<body>

<style>
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@500;700;900&display=swap');
        :root {
            --pale-blue: hsl(225, 100%, 94%);
            --bright-blue: hsl(245, 75%, 52%);
            --very-pale-blue: hsl(225, 100%, 98%);
            --desaturated-blue: hsl(224, 23%, 55%);
            --dark-blue: hsl(223, 47%, 23%);
        }
        body {
            font-family: 'Red Hat Display', sans-serif;
            font-size: 16px;
            position: relative;
            width: 100%;
            height: 100vh;
            padding: 0px;
            margin: 0px;
            background: var(--pale-blue);
        }
        body::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            width: 100%;
            height: 100%;
            background: url(https://rvs-order-summary-component.netlify.app/images/pattern-background-desktop.svg);
            background-repeat: no-repeat;
            background-size: contain;
            background-position: top;
            z-index: -1;
        }
        main {
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: row;
            justify-content: center;
            align-items: center;
        }
        .card {
            width: 320px;
            min-height: 400px;
            margin: 60px auto;
            border-radius: 10px;
            background: white;
        }
        .card .card-header {
            width: 100%;
            height: 156px;
            border-radius: 10px 10px 0px 0px;
        }
        .card .card-header img {
            width: 100%;
            border-radius: 10px 10px 0px 0px;
        }
        .card .card-body {
            width: 100%;
            height: auto;
            padding: 25px;
            box-sizing: border-box;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        .card .card-body .card-title {
            width: 100%;
            font-weight: 900;
            color: var(--dark-blue);
            text-align: center;
            padding: 15px;
            box-sizing: border-box;
        }
        .card .card-body .card-text {
            width: 100%;
            color: var(--desaturated-blue);
            text-align: center;
            line-height: 25px;
            padding: 15px 0px;
            box-sizing: border-box;
        }
        .card .card-body .card-plan {
            display: flex;
            flex-direction: row;
            align-items: center;
            column-gap: 15px;
            background: var(--very-pale-blue);
            border-radius: 10px;
            padding: 15px;
            box-sizing: border-box;
        }
        .card .card-body .card-plan .card-plan-img {
            flex-grow: 1;
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: center;
        }
        .card .card-body .card-plan .card-plan-text {
            flex-grow: 6;
            display: flex;
            flex-direction: column;
            row-gap: 4px;
        }
        .card .card-body .card-plan .card-plan-text .card-plan-title {
            color: var(--dark-blue);
            font-weight: 900;
            font-size: 14px;
        }
        .card .card-body .card-plan .card-plan-text .card-plan-price {
            color: var(--desaturated-blue);
            font-size: 14px;
        }
        .card .card-body .card-plan .card-plan-link {
            flex-grow: 1;
        }
        .card .card-body .card-plan .card-plan-link a {
            color: var(--bright-blue);
            font-weight: 700;
            font-size: 14px;
            cursor: pointer;
        }
        .card .card-body .card-plan .card-plan-link a:hover {
            color: #766cf1;
            text-decoration: none;;
        }
        .card .card-body .card-payment-button {
            padding: 25px 0px 15px;
            box-sizing: border-box;
        }
        .card .card-body .card-payment-button button {
            width: 100%;
            height: 50px;
            border: 0;
            background: var(--bright-blue);
            color: white;
            font-weight: 700;
            border-radius: 10px;
            box-shadow: 0px 10px 20px 0px hsl(245deg 75% 52% / 44%);
            cursor: pointer;
        }
        .card .card-body .card-payment-button button:hover {
            background: #766cf1;
        }
        .card .card-body .card-cancel-button {
            padding: 15px 0px;
            box-sizing: border-box;
        }
        .card .card-body .card-cancel-button button {
            width: 100%;
            border: 0;
            background: none;
            color: var(--desaturated-blue);
            font-weight: 900;
            text-align: center;
            cursor: pointer;
        }
        .card .card-body .card-cancel-button button:hover {
            color: var(--dark-blue);
        }
        

        @media (max-width: 375px) {
            body {
                height: auto;
            }
            body::before {
                content: "";
                position: absolute;
                top: 0;
                left: 0;
                right: 0;
                width: 100%;
                height: 100%;
                background: url(https://rvs-order-summary-component.netlify.app/images/pattern-background-mobile.svg);
                background-repeat: no-repeat;
                background-size: contain;
                background-position: top;
                z-index: -1;
            }
            
        }


</style>


</body>
<main>
        <div class="card">
            <div class="card-header">
                <img  width="450" height="220" src="https://westinpay.com/westin.png" alt="">
            </div>
            <div class="card-body">
                <div class="card-title">Order Summary</div>
                <div class="card-text"> Your WestinPay payment summary.</div>
                <div class="card-plan">
                    
                    <div class="card-plan-text">
                        <div class="card-plan-title">Annual Plan</div>
                        <div class="card-plan-price">$999.00/year</div>
                    </div>
           
                </div>
                <div class="card-payment-button">
                    <button onclick="location.href='https://westinpay.com/invoice/payment/eyJpdiI6IjdQV2l3ZVlFbGNXLzFaa1RsaHA0SUE9PSIsInZhbHVlIjoiSXVRa21FUzVYNFowOFBLbEtUWjZBayt6T1ZKd0ZlYWpZdzdFV0phK0hJbz0iLCJtYWMiOiIxMjQzYWYxYjQ5MzEzYzdiZGY4OTFhMWNkNzZlMjg0OGJlOWVmYTczZmM2OWM1NGE4MjRjMDIxMDk0ZDE1YzMyIiwidGFnIjoiIn0='" >Proceed to Payment</button>
                </div>
                <div class="card-cancel-button">
                    <button onclick="location.href='http://www.yoursite.com'" >Cancel Order</button>
                </div>
            </div>
        </div>
    </main>


</html
