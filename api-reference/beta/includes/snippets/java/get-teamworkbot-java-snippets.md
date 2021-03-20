---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57a432d3027b468c5b35c6a87b1c60d3276f1cda
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972251"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkBot teamworkBot = graphClient.appCatalogs().teamsApps("e4c5c249-bb4b-419e-b7c5-b1d98559368b").appDefinitions("ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk").bot()
    .buildRequest()
    .get();

```