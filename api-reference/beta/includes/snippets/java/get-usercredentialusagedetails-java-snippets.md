---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab70b0bab529ebd2429de64ce64072d67ddefe6fd9aec23c59ca11189d11699b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274323"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCredentialUsageDetailsCollectionPage userCredentialUsageDetails = graphClient.reports().userCredentialUsageDetails()
    .buildRequest()
    .get();

```