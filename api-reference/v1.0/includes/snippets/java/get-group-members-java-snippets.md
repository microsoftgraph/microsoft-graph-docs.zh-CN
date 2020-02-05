---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7fd9e249e0ab6846713dd1eba99b904f551edc9
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774538"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage members = graphClient.groups("{id}").members()
    .buildRequest()
    .get();

```