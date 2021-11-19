---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a20555ab1d554761db83bb9c9c3c0cd7cc597fb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.TermStore().GroupsById(&groupId).Sets().Get(options)


```