---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e2274bd6745649e1c3eb39ac4e6748fa29ac2f8b49b2ae6a0bebb90c76813ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333399"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = graphClient.me().onenote().sections("{id}")
    .buildRequest()
    .get();

```