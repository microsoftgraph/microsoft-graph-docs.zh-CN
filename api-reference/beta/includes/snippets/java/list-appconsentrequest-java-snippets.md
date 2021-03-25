---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4845668314d3ecc3d6d9569c1cda6af0e7b11cb3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201158"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequestCollectionPage appConsentRequests = graphClient.identityGovernance().appConsent().appConsentRequests()
    .buildRequest()
    .get();

```