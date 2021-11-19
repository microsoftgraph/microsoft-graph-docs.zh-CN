---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31d2d99360d71a6d569adcd6babd56a49995132d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100087"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationUserId := "educationUser-id"
graphClient.Education().UsersById(&educationUserId).Delete(options)


```