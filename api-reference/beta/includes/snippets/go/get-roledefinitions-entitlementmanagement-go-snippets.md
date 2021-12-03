---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a88ce1cbd8b80aa6bf33a261333ae584046084e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61289096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().EntitlementManagement().RoleDefinitions().Get(nil)


```