---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bee45e3bc9a8ba23769edcff6a6dc073177b4725
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099849"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().CloudPC().RoleDefinitions().Get(options)


```