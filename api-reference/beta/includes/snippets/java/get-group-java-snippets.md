---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aae5fd30a3d317fac3bb16ee34e44eae1805494
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945063"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage groups = graphClient.termStore().groups()
    .buildRequest()
    .get();

```