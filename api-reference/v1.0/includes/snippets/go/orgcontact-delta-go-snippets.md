---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaf7c2028bb4756a788bf900eede6a85a0eb338d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137722"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Contacts().Delta()().Get(nil)


```