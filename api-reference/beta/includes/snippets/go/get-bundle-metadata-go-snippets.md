---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80982a0e4766116db0e25d81c506ba4314573385
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
result, err := graphClient.Drive().BundlesById(&driveItemId).Get(options)


```