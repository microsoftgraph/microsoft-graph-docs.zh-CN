---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa0802a25b834f479833a028b56654d6283bb710
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094914"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviews().Get(options)


```