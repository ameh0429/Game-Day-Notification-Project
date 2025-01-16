# Game Day Notification Project

## Overview
The Game Day Notification Project is a real-time alert system that provides NBA game day score updates to subscribed users via SMS or email. By leveraging various AWS services and APIs, the project ensures sports fans stay up-to-date with the latest game information through an efficient and scalable notification mechanism.

## Features
- **Real-Time Alerts**: Delivers game day score notifications as they happen.
- **Multiple Channels**: Supports notifications via SMS and email.
- **Scalability**: Built on AWS services for high performance and scalability.
- **Customizable Subscriptions**: Allows users to subscribe to their preferred notification channel.

## Architecture
The project is powered by the following technologies and AWS services:

1. **Amazon SNS**: Sends notifications to users via SMS or email.
2. **AWS Lambda**: Processes game data and triggers notifications.
3. **Amazon EventBridge**: Orchestrates event-driven workflows and schedules Lambda functions.
4. **NBA APIs**: Fetches real-time game day scores and updates.
5. **Python**: Serves as the primary programming language for backend logic and API integration.

## Project Workflow
1. **Game Data Collection**: NBA APIs provide live score data.
2. **Event Triggering**: EventBridge schedules and triggers AWS Lambda functions.
3. **Data Processing**: Lambda functions process the game data and format notifications.
4. **Notification Delivery**: SNS sends the formatted notifications to subscribed users.

## Prerequisites
- An AWS account with access to SNS, Lambda, and EventBridge.
- Basic knowledge of Python and AWS services.
- NBA API credentials for accessing game day data.

## Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ameh0429/Game-Day-Notification-Project.git
   cd Game-Day-Notification-Project
   ```
2. **Configure AWS**:
   - Set up IAM roles and permissions for Lambda and SNS.
   - Create an SNS topic for notifications.
3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Set Up Environment Variables**:
   Create a `.env` file with the following details:
   ```env
   AWS_REGION=your-aws-region
   NBA_API_KEY=your-nba-api-key
   SNS_TOPIC_ARN=your-sns-topic-arn
   ```
5. **Deploy Lambda Functions**:
   Package and upload the Lambda function code to AWS.
6. **Configure EventBridge**:
   Create rules to trigger Lambda functions based on game schedules.

## Usage
1. Subscribe to the SNS topic via email or phone number.
2. Receive real-time notifications during NBA game days.

## Contributions
Contributions are welcome! Feel free to fork the repository, submit pull requests, or suggest features through the [issues page](https://github.com/ameh0429/Game-Day-Notification-Project/issues).

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Thanks to [NBA APIs](https://www.nba.com/) for providing real-time game data.
- Special appreciation to AWS for their robust cloud services.

---

For any questions or feedback, please contact the project maintainer at [ameh0429](https://github.com/ameh0429).
