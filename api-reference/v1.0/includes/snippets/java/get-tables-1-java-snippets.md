---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: debb2433b0ca23dd9e1f6b77f3495f543bb5678e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943311"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookTableCollectionPage tables = graphClient.me().drive().items("{id}").workbook().tables()
    .buildRequest()
    .get();

```