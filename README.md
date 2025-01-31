# CaltrainNext

A project that allows you to text the name of a Caltrain station and receive the next hour's worth of trains arriving at that station. This makes it really convenient to know how close the trains are to the station where you are waiting.

## Usage

To use the Caltrain Notifier, you will need to set up a Google Cloud Function and configure it to run the code in this repository. You will also need to set up a Twilio account and configure it to send and receive text messages.

## Installation

To get started with the Caltrain Notifier, you will need to clone this repository and install the requirements listed in the `requirements.txt` file in the `caltrain_response` folder. Here's how to do it:

1. Clone the repository: `git clone https://github.com/tyler-simons/caltrain-notifier.git`
2. Navigate to the `caltrain_response` folder: `cd caltrain_response`
3. Install the requirements: `pip install -r requirements.txt`

Once you have installed the requirements, you can play around with the script locally.

You can also deploy the function like this once you've set up your google cloud tools. See the file `deploy_caltrain_check.sh` for an example of what your deploy script could look like. You'll need to configure the options for yourself. This will deploy the function to Google Cloud, and you will be able to access it via the HTTP trigger URL provided by Google Cloud, which can trigger the Twilio function.

## Contributing

We welcome additions from the community. Please create an issue or make a PR to add something.

## License

MIT
