---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9208c381c9c57c00171f14a44e3d467dea996f0e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882245"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChannelCollectionPage channels = graphClient.teams("{id}").channels()
    .buildRequest()
    .get();

```