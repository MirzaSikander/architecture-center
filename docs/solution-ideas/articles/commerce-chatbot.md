---
title: Commerce Chatbot
titleSuffix: Azure Solution Ideas
author: adamboeglin
ms.date: 12/16/2019
description: Together, the Azure Bot Service and Language Understanding service enable developers to create conversational interfaces for various scenarios like banking, travel, and entertainment. For example, a hotel's concierge can use a bot to enhance traditional e-mail and phone call interactions by validating a customer via Azure Active Directory and using Cognitive Services to better contextually process customer requests using text and voice. The Speech recognition service can be added to support voice commands.
ms.custom: acom-architecture, chatbot, bot service, luis, interactive-diagram, 'https://azure.microsoft.com/solutions/architecture/commerce-chatbot/'
ms.service: architecture-center
ms.subservice: solution-idea
---

# Commerce Chatbot

[!INCLUDE [header_file](../header.md)]

Together, the Azure Bot Service and Language Understanding service enable developers to create conversational interfaces for various scenarios like banking, travel, and entertainment. For example, a hotel's concierge can use a bot to enhance traditional e-mail and phone call interactions by validating a customer via Azure Active Directory and using Cognitive Services to better contextually process customer requests using text and voice. The Speech recognition service can be added to support voice commands.

## Architecture

![Architecture diagram](../media/commerce-chatbot.svg)

## Data Flow

1. Customer uses your mobile app
1. Using Azure AD B2C, the user authenticates
1. Using the custom Application Bot, user requests information
1. Cognitive Services helps process the natural language request
1. Response is reviewed by customer who can refine the question using natural conversation
1. Once the user is happy with the results, the Application Bot updates the customer's reservation
1. Application insights gathers runtime telemetry to help development with Bot performance and usage
