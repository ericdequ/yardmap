Here's a detailed outline of the file structure and components for the YardMapp app using Expo:

```
YardMapp/
├── App.js
├── app.json
├── package.json
├── assets/
│   ├── images/
│   │   ├── logo.png
│   │   ├── homeowner.jpg
│   │   └── provider.jpg
│   └── fonts/
│       ├── Roboto-Regular.ttf
│       └── Roboto-Bold.ttf
├── src/
│   ├── components/
│   │   ├── HomeownerProfile/
│   │   │   ├── ProfileForm.js
│   │   │   ├── PropertyDetails.js
│   │   │   └── YardMap.js
│   │   ├── ProviderProfile/
│   │   │   ├── ProfileForm.js
│   │   │   ├── PortfolioGallery.js
│   │   │   └── ProviderServices.js
│   │   ├── ServiceRequest/
│   │   │   ├── RequestForm.js
│   │   │   ├── DatePicker.js
│   │   │   └── TimeSlotPicker.js
│   │   ├── ProviderList/
│   │   │   ├── ProviderCard.js
│   │   │   ├── ProviderDetails.js
│   │   │   └── RatingStars.js
│   │   ├── Messaging/
│   │   │   ├── MessageList.js
│   │   │   ├── MessageInput.js
│   │   │   └── ChatScreen.js
│   │   ├── UI/
│   │   │   ├── Button.js
│   │   │   ├── Input.js
│   │   │   ├── Text.js
│   │   │   └── Icon.js
│   │   └── index.js
│   ├── screens/
│   │   ├── HomeownerScreens/
│   │   │   ├── HomeScreen.js
│   │   │   ├── ProfileScreen.js
│   │   │   ├── YardMapScreen.js
│   │   │   ├── ServiceRequestScreen.js
│   │   │   ├── ProviderListScreen.js
│   │   │   └── MessagingScreen.js
│   │   ├── ProviderScreens/
│   │   │   ├── DashboardScreen.js
│   │   │   ├── ProfileScreen.js
│   │   │   ├── ServiceRequestsScreen.js
│   │   │   └── MessagingScreen.js
│   │   ├── AuthScreens/
│   │   │   ├── LoginScreen.js
│   │   │   └── SignupScreen.js
│   │   └── index.js
│   ├── navigation/
│   │   ├── HomeownerNavigator.js
│   │   ├── ProviderNavigator.js
│   │   └── AuthNavigator.js
│   ├── api/
│   │   ├── homeownerApi.js
│   │   ├── providerApi.js
│   │   └── messagingApi.js
│   ├── utils/
│   │   ├── colors.js
│   │   ├── constants.js
│   │   └── helpers.js
│   └── App.js
├── .gitignore
├── .expo/
│   ├── packager-info.json
│   └── settings.json
└── README.md
```

Here's a breakdown of the main files and components:

- `App.js`: The entry point of the application where the main component is rendered.
- `app.json`: The configuration file for the Expo app.
- `package.json`: The file containing project dependencies and scripts.
- `assets/`: The directory for storing static assets such as images and fonts.
  - `images/`: Contains images used in the app (e.g., logo, homeowner, provider).
  - `fonts/`: Contains custom fonts used in the app (e.g., Roboto).
- `src/`: The main directory for the application source code.
  - `components/`: Contains reusable components used throughout the app.
    - `HomeownerProfile/`: Components related to the homeowner's profile.
      - `ProfileForm.js`: Renders the form for homeowners to update their profile information.
      - `PropertyDetails.js`: Displays the details of the homeowner's property.
      - `YardMap.js`: Allows homeowners to map out their yard's sprinkler system and lighting setup.
    - `ProviderProfile/`: Components related to the service provider's profile.
      - `ProfileForm.js`: Renders the form for service providers to update their profile information.
      - `PortfolioGallery.js`: Displays the service provider's portfolio images.
      - `ProviderServices.js`: Lists the services offered by the service provider.
    - `ServiceRequest/`: Components related to service requests.
      - `RequestForm.js`: Renders the form for homeowners to request yard maintenance or landscaping services.
      - `DatePicker.js`: Allows homeowners to select the desired service date.
      - `TimeSlotPicker.js`: Allows homeowners to choose a time slot for the service.
    - `ProviderList/`: Components related to the list of service providers.
      - `ProviderCard.js`: Renders a card displaying a service provider's information.
      - `ProviderDetails.js`: Displays detailed information about a service provider.
      - `RatingStars.js`: Renders rating stars based on the service provider's ratings.
    - `Messaging/`: Components related to messaging and communication.
      - `MessageList.js`: Renders the list of messages in a conversation.
      - `MessageInput.js`: Allows users to input and send messages.
      - `ChatScreen.js`: Displays the chat screen for a conversation between a homeowner and a service provider.
    - `UI/`: Contains reusable UI components.
      - `Button.js`: Renders a custom button component.
      - `Input.js`: Renders a custom input component.
      - `Text.js`: Renders a custom text component.
      - `Icon.js`: Renders custom icons used in the app.
    - `index.js`: Exports all the components for easy importing.
  - `screens/`: Contains the main screens of the app.
    - `HomeownerScreens/`: Screens specific to homeowners.
      - `HomeScreen.js`: Displays the homeowner's home screen with relevant information and options.
      - `ProfileScreen.js`: Allows homeowners to view and update their profile information.
      - `YardMapScreen.js`: Displays the yard mapping screen for homeowners to map their sprinkler system and lighting setup.
      - `ServiceRequestScreen.js`: Allows homeowners to request yard maintenance or landscaping services.
      - `ProviderListScreen.js`: Displays the list of service providers available for the homeowner's location.
      - `MessagingScreen.js`: Displays the messaging screen for homeowners to communicate with service providers.
    - `ProviderScreens/`: Screens specific to service providers.
      - `DashboardScreen.js`: Displays the service provider's dashboard with relevant information and options.
      - `ProfileScreen.js`: Allows service providers to view and update their profile information.
      - `ServiceRequestsScreen.js`: Displays the list of service requests received by the service provider.
      - `MessagingScreen.js`: Displays the messaging screen for service providers to communicate with homeowners.
    - `AuthScreens/`: Screens related to authentication.
      - `LoginScreen.js`: Renders the login screen for users to sign in to the app.
      - `SignupScreen.js`: Renders the signup screen for users to create a new account.
    - `index.js`: Exports all the screens for easy importing.
  - `navigation/`: Contains the navigation setup for the app.
    - `HomeownerNavigator.js`: Defines the navigation flow for homeowners.
    - `ProviderNavigator.js`: Defines the navigation flow for service providers.
    - `AuthNavigator.js`: Defines the navigation flow for authentication screens.
  - `api/`: Contains the API handlers for making requests to the backend server.
    - `homeownerApi.js`: Handles API requests related to homeowners.
    - `providerApi.js`: Handles API requests related to service providers.
    - `messagingApi.js`: Handles API requests related to messaging and communication.
  - `utils/`: Contains utility functions and constants used throughout the app.
    - `colors.js`: Defines the color palette used in the app.
    - `constants.js`: Defines constant values used in the app.
    - `helpers.js`: Contains helper functions used in the app.
  - `App.js`: The main component that sets up the app navigation and screens.
- `.gitignore`: Specifies files and directories to be ignored by Git.
- `.expo/`: Contains Expo-related configuration files.
- `README.md`: Provides information and instructions about the project.

To set up the project with Expo, follow these steps:

1. Install Expo CLI globally: `npm install -g expo-cli`
2. Initialize a new Expo project: `expo init YardMapp`
3. Choose the "blank" template when prompted.
4. Navigate to the project directory: `cd YardMapp`
5. Create the necessary directories and files as outlined in the file structure above.
6. Implement the components, screens, and navigation according to the app's requirements.
7. Set up the backend API and integrate it with the app.
8. Implement user authentication and authorization.
9. Test the app using Expo's development server: `expo start`
10. Follow the Expo CLI instructions to run the app on an emulator/simulator or physical device.

Remember to handle edge cases, error scenarios, and loading states throughout the app. Implement proper state management using React hooks, context, or libraries like Redux or MobX.

Regularly test the app on different devices and platforms to ensure compatibility and a smooth user experience. Optimize performance by implementing lazy loading, caching, and efficient data fetching strategies.

Follow Expo's documentation and best practices for building and deploying your app. Consider implementing push notifications, analytics, and crash reporting to enhance the app's functionality and gather user insights.

Finally, ensure that the app follows accessibility guidelines and provides a user-friendly interface for all users, including those with disabilities.