---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cfb25d63ea32824791277cd498a21e67ea11585
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014286"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviews().Get(options)


```