---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bb62a836623911c1f31afc5f71f9a160a95e93f74f73012323dd5ed6ab9fe77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274430"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .buildRequest()
    .delete();

```