---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9136684298fd9c86af6773c68ec27f21e85f12d92f5cec8dc97fbf49cdebf72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278810"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpoint printServiceEndpoint = graphClient.print().services("{printServiceId}").endpoints("{printServiceEndpointId}")
    .buildRequest()
    .get();

```