---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ea3599e1152b8ecede561fb9bf382c49f25545b
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006669"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteCollectionPage followedSites = graphClient.me().followedSites()
    .buildRequest()
    .get();

```