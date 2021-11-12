---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdaec9130baff1dd5ece7c93354d2c6d06ef63b1e977e3e26c3721f7369ec9df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104760"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("86b6d420-7e6b-4797-a05c-af4e56cd81bd").jobs("31216")
    .buildRequest()
    .expand("documents")
    .get();

```