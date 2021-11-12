---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d658735f7bf452cbb75c89c406bb3835fa8e6ee1e9c3baaa70d63482087ec58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = graphClient.print().printers("{id}")
    .buildRequest()
    .get();

```