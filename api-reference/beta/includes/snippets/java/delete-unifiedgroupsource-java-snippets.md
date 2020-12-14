---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26bca4b589b9a048e477eef0876cfcf17e678114
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657145"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{ediscoveryCaseId}").custodians("{custodianId}").unifiedGroupSources("{unifiedGroupSourceId}")
    .buildRequest()
    .delete();

```