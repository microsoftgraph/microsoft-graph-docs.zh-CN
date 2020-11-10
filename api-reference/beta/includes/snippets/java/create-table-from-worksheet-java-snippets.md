---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f04a48f39f36e2aaf1c6b666fbabcd013597747
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977246"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "";

Boolean hasHeaders = false;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").tables()
    .add(address,hasHeaders)
    .buildRequest()
    .post();

```