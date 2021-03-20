---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 831243506c58f536d3b203ff86c1a97c75c8a97c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy").includes("198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5")
    .buildRequest()
    .delete();

```