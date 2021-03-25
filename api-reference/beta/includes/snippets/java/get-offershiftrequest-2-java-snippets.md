---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 671540cc182194128c2ac3489d6558cb99464505
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209179"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OfferShiftRequestCollectionPage offerShiftRequests = graphClient.teams("{teamId}").schedule().offerShiftRequests()
    .buildRequest()
    .get();

```