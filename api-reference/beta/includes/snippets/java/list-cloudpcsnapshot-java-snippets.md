---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 530677126a5d365280b63c4885b02ccf0801e4fd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335323"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcSnapshotCollectionPage snapshots = graphClient.deviceManagement().virtualEndpoint().snapshots()
    .buildRequest()
    .get();

```