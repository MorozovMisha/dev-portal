# Introduction to SingularityNET Ecosystem

## Ecosystem consists of [Decentralized AI Platform](/docs/products/DecentralizedAIPlatform/) and [AI Marketplace](/docs/products/AIMarketplace/).

## SingularityNET Marketplace

[The SingularityNET Marketplace](http://beta.singularitynet.io) is a decentralized application (DApp), which lists the available AI services and helps you to interact with those services through web interface abstracting all the complexity in invoking a service. It also processes payment for services (through MetaMask/General Wallet) and conduct service ratings.
Whenever transaction happens on Blockchain, an event is created. The marketplace monitors all those events.
For example, if you publish a new organization, a new service, the marketplace receives an alert notification about published information in the Blockchain. The marketplace reads the organization metadata, the service metadata and stores this into its database. This application efficiently displays all the details quickly without relying on the slow performance of the Blockchain.

The following image shows the contents from the marketplace.

<ImageViewer src="/assets/images/products/AIMarketplace/forcomers/dapp_landing_page.webp" alt="marketplace"/>

The decentralized application (DApp) does the following:

-   Reads data from the on-chain Registry and pairs it with off-chain metadata.
    This allows for searching, filtering, and discovering AI services.

-   Integrates the SingularityNET curation service, and displays from the registry.
    Whenever an event comes from Blockchain, the details are stored in the local database, the review process is done on that data, and then when approved, the information is made available in the marketplace.
    **Note:** Displays those services that have been vetted, and owners who have experienced due diligence and signed legal agreements that protects user and data privacy.

-   Displays custom UI components for interactions with AI services.
    It enables you to quickly build the UI components and host the component on the platform, and also you can determine what inputs need to be chosen for service execution, and is the expected output, without understanding the complexity of knowing the gRPC protocol, the proto that is associated with the service and how to call the service and so on.

-   Integrates with Multi-Party Escrow, to allow consumers to pay for service usage;
    Allows consumers to rate the utilized services.
    **Note:** This rating services will be part of the SingularityNET's Reputation System (currently under development). Currently, it is very difficult to rate services on Blockchain. Therefore all rating mechanisms are performed off-chain and managed in the market place. So you can share your opinion and reviews at marketplace.

-   Captures usage metrics at a consumer level.

**Note:** Although, the SingularityNET platform is open and decentralized, the Marketplace is the SingularityNET Foundation's curated view. This allows the foundation to adhere to legal requirements of different legislative regions. Currently, the Marketplace and SingularityNET is in beta stage. For more information about the current status, refer to current status page for changes, or follow the [git-repo](https://github.com/singnet/snet-dapp)

## Marketplace Requirements

If you are a service author, for the service to be visible to others and listed on the marketplace you must:

1. Build and publish your service
2. Use SSL with the snet-daemon.
   **Note:** if you don't already have an SSL certificate for your domain, it is recommended you use certbot and letsencrypt .
3. Fork the snet-dapp repo, build a react component as the user interface for your service, and submit a pull request.
   **Note:** Identify the services on your networks, organization and service names being used. For more details, refer to dapp repo README.md.
4. Last is some paperwork that we are still finalising, and we'll update this list when we have that. If you are itching to get your service listed, reach out to us via one of our community groups.
   **Note:** your service can be published to SingularityNET without being listed on the marketplace, but your service may be less discoverable to potential customers if it is not listed.
