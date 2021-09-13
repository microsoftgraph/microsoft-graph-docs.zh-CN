---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b415a0fd37069a21125bf272bacbf0736b1140c88bb9d8c867fe73147b8cd7e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333896"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .delete();

```