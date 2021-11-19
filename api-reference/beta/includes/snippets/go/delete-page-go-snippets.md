---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac8518e4d7fa3f83c406a9d53370ae949aefcf9b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083458"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onenotePageId := "onenotePage-id"
graphClient.Me().Onenote().PagesById(&onenotePageId).Delete(options)


```