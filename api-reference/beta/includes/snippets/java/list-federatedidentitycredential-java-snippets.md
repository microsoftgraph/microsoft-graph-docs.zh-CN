---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6c6b159d1263167e06b8d3fbeb3a2cc7a34a4af
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689197"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FederatedIdentityCredentialCollectionPage federatedIdentityCredentials = graphClient.applications("bcd7c908-1c4d-4d48-93ee-ff38349a75c8").federatedIdentityCredentials()
    .buildRequest()
    .get();

```