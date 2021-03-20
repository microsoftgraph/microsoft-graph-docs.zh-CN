---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72f877cdbb40654890e8b79cca4637739a3ceb34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975425"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProvisioningObjectSummaryCollectionPage provisioning = graphClient.auditLogs().provisioning()
    .buildRequest()
    .get();

```