---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e66e095a97dbbf449bbfce93d3cc6e0b8026dff2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881264"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookWorksheetCollectionPage worksheets = graphClient.me().drive().items("{id}").workbook().worksheets()
    .buildRequest()
    .get();

```