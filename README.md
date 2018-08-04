<html>
	<head>
		
		<title>About ForkDelta | Roadmap, FAQs, and more!</title>
		<meta name="description" content="Learn about ForkDelta today! ForkDelta is a fully decentralized Ethereum Token Exchange with the most ERC20 listings of any exchange." />
		
		<meta property="og:url" content="https://forkdelta.github.io" />
	    <meta property="og:title" content="About ForkDelta | Roadmaps, FAQs, and more!" />
	    <meta property="og:description" content="Learn about ForkDelta today! ForkDelta is a fully decentralized Ethereum Token Exchange with the most ERC20 listings of any exchange." />
	    <meta property="og:image" content="https://forkdelta.github.io/images/logo.png" />

		<link type="text/css" rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" />
		<script src="https://code.jquery.com/jquery-3.3.1.min.js"
				integrity="sha256-FgpCb/KJQlLNfOu91ta32o/NMZxltwRo8QtmkMRdAu8="
				crossorigin="anonymous"></script>

		<script>
			
			$(document).ready(function($) {

				//if page loaded with a hash, smooth scroll to it
				if (window.location.hash !== '') {
					scroll_to_hash(window.location.hash);
				}

				//bind accordion
				$('#faqs').find('.accordion-toggle').click(function(){

					//Expand or collapse this panel
					$(this).next().slideToggle('fast');

					//Hide the other panels
					$(".accordion-content").not($(this).next()).slideUp('fast');

				});

				// Add smooth scrolling to nav links
				$("a.hash").on('click', function(event) {
					event.preventDefault();

					scroll_to_hash(this.hash);

					window.location.hash = this.hash;
				});
			});

			function scroll_to_hash(hash) {
				if (hash === '#roadmap') {
					var offsettop = 0;
				} else {
					var offsettop = $('a[name="' + hash + '"]').offset().top;
				}

				$('html, body').animate({
					scrollTop: offsettop,
				}, 1000);
			}

		</script>

		<style>
			* {
				box-sizing: border-box;
			}

			body {
				background: #f7f7f7;
				font-family: Segoe UI;
				padding: 70px 0;
			}

			h1 {
			  text-align: center;
			  font-size: 3rem;
			  font-weight: 200;
			  margin-bottom: 20px;
			}

			h2 {
				text-align: center;
				font-size: 2rem;
				font-weight: 200;
			}

			a {
				text-decoration: none;
			}
			
			img {
				width: 100%;
			}

			.header {
			    position: fixed;
			    top: 0;
			    left: 0;
			    width: 100%;
			    text-align: center;
			    /* position: relative; */
			    z-index: 9;
			    background: #FFF;
			    box-shadow: 0px 1px 22px 4px rgba(0, 0, 0, 0.07);
			}

			.header a {
			    padding: 20px 30px;
			    display: inline-block;
			    text-decoration: none;
			    color: #394b59;
			}

			.header a:hover {
				color: #fe5f2c;
			}

			.content {
				width: 1000px;
				margin: 0 auto;
				border:1px solid #E0E0E0;
				padding:12px;
				color:#212121;
				background:#FFF;
				font-size:15px;
				line-height:1.45em;
				box-shadow: 0px 1px 22px 4px rgba(0, 0, 0, 0.07);
			}

			/* accordion css */
			#faqs {
				width: 1000px;
				box-shadow: 0px 1px 22px 4px rgba(0, 0, 0, 0.07);
				margin: 0 auto;
			}

			.accordion-toggle,
			.accordion-content {
				width: 100%;
				margin: 0 auto;
			}

			.accordion-toggle {
				cursor: pointer;
				background:#394b59;
				padding:12px;
				cursor:pointer;
				border-right:1px solid #2d3d4a;
				border-left:1px solid #2d3d4a;
				border-bottom:1px solid #2d3d4a;
				min-height:20px;
				transition:.25s;

				font-size:18px;
				font-weight: normal;
				line-height: 1.3em;
				color:#ffffff;
			}

			.accordion-content {
				display: none;
				border-left:1px solid #E0E0E0;
				border-right:1px solid #E0E0E0;
				border-bottom:1px solid #E0E0E0;
				padding:12px;
				color:#212121;
				background:#FFF;
				font-size:15px;
				line-height:1.45em;
			}

			.accordion-content.open { display: block; }

			/* timeline css */
			.timeline .demo-card-wrapper {
			  position: relative;
			  margin: auto;
			}
			.timeline .demo-card-wrapper::after {
			  z-index: 1;
			  content: "";
			  position: absolute;
			  top: 0;
			  bottom: 0;
			  left: 50%;
			  border-left: 1px solid rgba(191, 191, 191, 0.4);
			}
			.timeline .demo-card {
			  position: relative;
			  display: block;
			  margin: 10px auto;
			  z-index: 2;
			  max-width: 1000px;
			  box-shadow: 0px 1px 22px 4px rgba(0, 0, 0, 0.07);
			}
			.timeline .demo-card .head {
			  position: relative;
			  display: flex;
			  align-items: center;
			  color: #fff;
			  font-weight: 400;
			}
			.timeline .demo-card .head .number-box {
			  display: inline;
			  float: left;
			  margin: 15px;
			  padding: 10px;
			  font-size: 35px;
			  line-height: 35px;
			  font-weight: 600;
			  background: rgba(0, 0, 0, 0.17);
			}
			.timeline .demo-card .head h2 {
			  font-size: 24px;
			  font-weight: inherit;
			  letter-spacing: 2px;
			  margin: 0;
			  padding-bottom: 6px;
			  line-height: 26px;
			  text-align: left;
			}
			.timeline .demo-card .head h2 span {
			  display: block;
			  font-size: 18px;
			  text-transform: uppercase;
			  margin: 0;
			}
			@media (min-width: 480px) {
			  .timeline .demo-card .head h2 span {
			    font-size: 0.8rem;
			  }
			}

			.timeline .demo-card {
				background: #394b59;
			}

			.timeline .demo-card.green {
				background: #77DD77;
			}

		</style>
	</head>

	<body>

		<div class="header">
			<a href="https://forkdelta.github.io">Trade</a>
			<a class="hash" href="#roadmap">Roadmap</a>
			<a class="hash" href="#donate">Donate</a>
			<a class="hash" href="#faqs">FAQs</a>
		</div>

		<a name="#roadmap"></a>
		<h1>ForkDelta Roadmap</h1>

		<section class=timeline>
			<div class="demo-card-wrapper">
				<div class="demo-card green">
					<div class="head">
						<div class="number-box">
							<span><i class="fa fa-check"></i></span>
						</div>
						<h2><span class="small">January 5th 2018</span> Fork EtherDelta</h2>
					</div>
				</div>

				<div class="demo-card green">
					<div class="head">
						<div class="number-box">
							<span><i class="fa fa-check"></i></span>
						</div>
						<h2><span class="small">January 24th 2018</span> Simplify Token Submission Process</h2>
					</div>
				</div>

				<div class="demo-card green">
					<div class="head">
						<div class="number-box">
							<span><i class="fa fa-check"></i></span>
						</div>
						<h2><span class="small">February 15th 2018</span> Launch New Order Processing Back End</h2>
					</div>
				</div>

				<div class="demo-card">
					<div class="head">
						<div class="number-box">
							<span>Q1<br />2018</span>
						</div>
						<h2>Launch New Public API</h2>
					</div>
				</div>

				<div class="demo-card">
					<div class="head">
						<div class="number-box">
							<span>Q1<br />2018</span>
						</div>
						<h2>Launch New Front End UI</h2>
					</div>
				</div>

				<div class="demo-card">
					<div class="head">
						<div class="number-box">
							<span>Q2<br />2018</span>
						</div>
						<h2><span class="small">Q2 or Q3 2018</span> New Smart Contract (possibly 0x)</h2>
					</div>
				</div>
		    
			</div>
		</section>

		<h2>Possible Future Changes</h2>

		<section class=timeline>
			<div class="demo-card-wrapper">
				<div class="demo-card">
					<div class="head">
						<div class="number-box">
							<span><i class="fa fa-question"></i></span>
						</div>
						<h2><span class="small">TBD</span> Tokenized Method of Platform Ownership</h2>
					</div>
				</div>

				<div class="demo-card">
					<div class="head">
						<div class="number-box">
							<span><i class="fa fa-question"></i></span>
						</div>
						<h2><span class="small">TBD</span> Decentralized Order Book</h2>
					</div>
				</div>

				<div class="demo-card">
					<div class="head">
						<div class="number-box">
							<span><i class="fa fa-question"></i></span>
						</div>
						<h2><span class="small">TBD</span> Decentralized Hosting</h2>
					</div>
				</div>
		    
			</div>
		</section>

		<a name="#donate"></a>
		<h1 style="margin-top: 120px;">Donate</h1>
		<div class="content">
			ForkDelta currently interfaces with EtherDelta's original smart contract which allows ForkDelta users to trade utilizing EtherDelta's volume. However, this means that the trading fees still go to EtherDelta and ForkDelta development costs come entirely out of our pockets. If you are interested in the ForkDelta project and would like to contribute to its future, please consider donating to the Ethereum address below.<br />
			<h2><a href="https://etherscan.io/address/0x25b9003b1935bcfba170b5b63780f265c2248f52">0x25B9003b1935bCFBA170B5B63780F265C2248F52</a></h2>
			As this is a project by the community, for the community, transactions to and from the donations address will be public and can be viewed on the blockchain. We will also keep a public ledger of how the donations are distributed. That way, donors can see exactly how their donations are helping!
		</div>

		<a name="#faqs"></a>
		<h1 style="margin-top: 120px;">Frequently Asked Questions</h1>

		<div id="faqs">

			<h4 class="accordion-toggle">What is ForkDelta?</h4>
			<div class="accordion-content open">
				ForkDelta is a decentralized Ethereum Token Exchange with the most ERC20 listings of any exchange. ForkDelta currently acts as an open source, updated interface for EtherDelta's smart contract with an active and public development team.
				<br /><br />
				The official URL is <a href="https://cryptodelta.github.io">https://cryptodelta.github.io</a>
			</div>

			<h4 class="accordion-toggle">What is a decentralized exchange?</h4>
			<div class="accordion-content">
				A decentralized exchange is an exchange that doesn't rely on a centralized party to store user's funds and facilitate trades.
				In ForkDelta's case, funds are stored in a smart contract hosted on the Ethereum network.
				Trades also occur directly between users using the same smart contract.
			</div>

			<h4 class="accordion-toggle">How is ForkDelta different from EtherDelta?</h4>
			<div class="accordion-content">
				ForkDelta started as a fork of EtherDelta when EtherDelta was sold to new owners who introduced questionable development decisions.
				Considerable development time has been put towards a new token listing system, order book, API, and front-end UI all of which are at different stages of development and can be tracked on <a href="https://github.com/forkdelta/">GitHub</a>.
				<br /><br />
				ForkDelta prides itself on being an open, fair community with developers who are easily accessed and an open source codebase.<br />
				At ForkDelta, we believe in direct and open streams of communication with the community.<br />
				We pride ourselves on our availability in our <a href="https://discord.gg/MPvAfMa">Discord channel</a> and through comments on GitHub pull requests and issues.<br />
				We welcome any feedback, criticism, ideas, and help that the community would like to give.<br />
				ForkDelta does not and will not ever charge fees for token listings.<br />
				ForkDelta also lists the most tokens of any exchange with new tokens added every day.<br />
			</div>

			<h4 class="accordion-toggle">How do I create an account?</h4>
			<div class="accordion-content">
				If you have an Ethereum wallet, you already have an account!
				Simply link your Ethereum wallet using either MetaMask, Ledger, or importing your account directly using the dropdown in the top right of the trading view. 
			</div>

			<h4 class="accordion-toggle">How do I deposit funds?</h4>
			<div class="accordion-content">
				After you've selected an account, depositing funds is easy! In the Deposit/Withdraw/Transfer window in the top left, select Deposit, then select the amount of either Ethereum or tokens you would like to deposit. You will then be asked to sign or accept the transaction. Once the transaction has been sent, your funds are deposited securely into the smart contract on the Ethereum network. Then, you'll be able to trade on ForkDelta with those funds!<br />
				For an example using MetaMask, watch the gif below.<br />
				<img src="https://forkdelta.github.io/images/deposit.gif" />
			</div>

			<h4 class="accordion-toggle">How do I withdraw funds?</h4>
			<div class="accordion-content">
				The withdrawal process is very similar to the deposit process. In the Deposit/Withdraw/Transfer window in the top left, select Withdraw, then select the amount of either Ethereum or tokens you would like to withdraw into the connected Ethereum account. You will then be asked to sign or accept the transaction. Once the transaction has been sent, your funds are withdrawn securely into your Ethereum account.<br />
				For an example using MetaMask, watch the gif below.<br />
				<img src="https://forkdelta.github.io/images/withdraw.gif" />
			</div>

			<h4 class="accordion-toggle">How long does it take to withdraw or deposit funds?</h4>
			<div class="accordion-content">
				As ForkDelta depends on a smart contract hosted on the Ethereum network, the speed of transactions depends entirely on the speed of the Ethereum network. If you would like deposits, withdrawals, trades, or orders to be processed faster, you can increase the gas price for your transactions. Under normal loads, with a normal gas price, deposits and withdrawals shouldn't take longer than 5 minutes. However, when the Ethereum network is clogged, transactions could be delayed.<br />
				<br />
				For informatino on the current state of the Ethereum network, please go to <a href="https://ethgasstation.info/">EthGasStation</a>.
			</div>

			<h4 class="accordion-toggle">How do I select a token?</h4>
			<div class="accordion-content">
				In ForkDelta, you can trade any ERC20 token that is available on the Ethereum network. We do our best to list as many tokens as possible. The listed tokens can be found in a dropdown near the upper left section of ForkDelta. If you navigate to ForkDelta's home page, the drop down should default to DAI.<br />
				<br />
				However, there is another way to select which token to trade that works even if we haven't listed the token yet!<br />
				Take a look at this URL: https://forkdelta.github.io/#!/trade/DAI-ETH<br />
				If you would like to trade a token that is not listed on ForkDelta, simply replace DAI with that tokens contract address.<br />
				Like so: https://forkdelta.github.io/#!/trade/0x12b306fa98f4cbb8d4457fdff3a0a0a56f07ccdf-ETH
			</div>

			<h4 class="accordion-toggle">How do I place an order?</h4>
			<div class="accordion-content">
				After funds have been placed in the smart contract, you are ready to place or take an order. If you would like to create a buy or sell order instead of taking an order that already exists, first, find the New Order section. Then, select either buy or sell and enter in the token amount you would like to buy or sell, the price, the expiration time, and hit Buy/Sell. You will then be prompted to sign the transaction, so that it can be sent to the order book. Once a taker for your order has been found, ForkDelta will use that signed order to execute a trade using the smart contract on the Ethereum network.
			</div>

			<h4 class="accordion-toggle">Where are the market orders?</h4>
			<div class="accordion-content">
				ForkDelta does not currently have market orders, but it is something that we are working on. For updates on our progress on market orders, please take a look at <a href="https://github.com/forkdelta/nextgen-ui/issues/13">this GitHub issue</a>.<br />
				We recommend specifying and taking existing orders to replicate a similar functionality to a market order.
			</div>

			<h4 class="accordion-toggle">How do I take an order?</h4>
			<div class="accordion-content">
				To take an existing order, simply click on the order you would like to take in the Order Book. You will be prompted with a window asking you to specify the amount you would like to take. After you hit the accompanying Buy or Sell button, you will then be prompted to sign the transaction, so that your trade can be sent to the smart contract. ForkDelta will give you a transaction ID and a link. You can track your trade status by either clicking the link, or copying the transaction ID and searching it on EtherScan.<br />
				Trades don't always show up immediately on EtherScan and the speed of the transaction depends on the Ethereum network's congestion and your set gas price.
			</div>

			<h4 class="accordion-toggle">How do I cancel an order?</h4>
			<div class="accordion-content">
				To cancel an order, take a look at the My Transactions section and click the Orders tab. Your active orders will be listed there with a link to cancel them. You will be asked to sign a transaction in order to cancel the order.<br />
				For an example using Metamask, watch the gif below:<br />
				<img src="https://forkdelta.github.io/images/cancel.gif" />
			</div>

			<h4 class="accordion-toggle">What fees are associated?</h4>
			<div class="accordion-content">
				There are two trading fees while using the ForkDelta platform. The first is the small Ethereum fee for signing transactions to the Ethereum network. The second is a 0.3% fee on execution of orders. 
			</div>

			<h4 class="accordion-toggle">Where are the trading fees going?</h4>
			<div class="accordion-content">
				The fee for signing transactions on the Ethereum network goes directly to the miners on the network.<br />
				As we are currently using EtherDelta's smart contract, the 0.3% fee is going to the EtherDelta team as specified in their smart contract. We hope to change this in the future, but would like to make sure we keep the necessary volume on this exchange.<br /><br />
				If you are interested in supporting the ForkDelta project, please consider donating.
			</div>

			<h4 class="accordion-toggle">How do I get my token listed on ForkDelta?</h4>
			<div class="accordion-content">
				Any member of the ForkDelta community can request a token to be listed on ForkDelta by filing <a href="https://github.com/forkdelta/tokenbase/issues/new">an issue</a>.
				<br /><br />
				More information on the token listing process is available <a href="https://www.reddit.com/r/ForkDelta/comments/7tntnz/how_to_get_an_erc20_token_listed_on_forkdelta/">here</a>.
			</div>

			<h4 class="accordion-toggle">How do I change the default gas price?</h4>
			<div class="accordion-content">
				To change the default gas price, simply click the drop down in the top right of ForkDelta (where you previously set up your account), and click "Gas Price" at the bottom of that menu. Then, you can set your gas price using the Gwei denomination.
			</div>

			<h4 class="accordion-toggle">How do I use a Ledger directly with ForkDelta?</h4>
			<div class="accordion-content">
				First, you need to make sure that browser support and contract support are enabled on your Ledger. To do so, navigate to the Ethereum app on your Ledger, go into settings, and enable both browser support and contract support. Then, make sure your Ledger is connected to your computer and navigate to ForkDelta. Your Ledger address will appear in the account dropdown automatically, with a green "Ledger" box next to it. When you deposit, withdraw, place an order, or trade, you will have to approve the transaction on your Ledger.
			</div>

		</div>
		
	</body>
</html>
