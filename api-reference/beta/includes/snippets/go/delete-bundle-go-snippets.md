---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eea7411189e1423a36d5bc8fc654d371c6779651
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088574"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Delete(options)


```