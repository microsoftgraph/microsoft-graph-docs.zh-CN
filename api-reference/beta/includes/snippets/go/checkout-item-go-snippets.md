---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c658ca1cd464d734a7db6bbb3b2a57b841fd4905
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093660"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
driveItemId := "driveItem-id"
graphClient.DrivesById(&driveId).ItemsById(&driveItemId).Checkout(drive-id, driveItem-id).Post()


```