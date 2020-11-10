---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e66e095a97dbbf449bbfce93d3cc6e0b8026dff2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982106"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookWorksheetCollectionPage worksheets = graphClient.me().drive().items("{id}").workbook().worksheets()
    .buildRequest()
    .get();

```