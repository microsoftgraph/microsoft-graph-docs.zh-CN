---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a963d03dc4f65ecd4148756dbe4e32933ffa75a7361b7b3d3700f34b54e9148b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105154"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").custodians("{custodianId}").unifiedGroupSources("{unifiedGroupSourceId}")
    .buildRequest()
    .delete();

```