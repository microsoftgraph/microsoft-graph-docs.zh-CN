---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec7a451be0806f56c7bd94088cc55ae4604b2fdd3d680feee7ddd86c381bf862
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("2eef613a-ca2d-42f4-89fe-84d5198ddedf").reviewSets("b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8").queries("6b5358b0-2ce2-4369-b9cf-65392fe56807")
    .buildRequest()
    .delete();

```