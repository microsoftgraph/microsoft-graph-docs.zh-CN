---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3c7828ef6c2abf139b817f42dd23a68f872b339
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100002"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Compliance().Ediscovery().Cases().Post(options)


```