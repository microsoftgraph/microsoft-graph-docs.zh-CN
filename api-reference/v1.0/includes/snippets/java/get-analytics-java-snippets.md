---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ea3599e1152b8ecede561fb9bf382c49f25545b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793909"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteCollectionPage followedSites = graphClient.me().followedSites()
    .buildRequest()
    .get();

```