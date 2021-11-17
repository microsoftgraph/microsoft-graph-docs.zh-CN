---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c47a9275cbd80b243684333cba07746b99fa0366db2f908065fe32ff7d587de4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163577"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkforceIntegrationCollectionPage workforceIntegrations = graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .get();

```