---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17e373bdb8c6c024a1d1cad54ce9ce8b938dce5b89380ec22ac877d6dae67dad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = graphClient.me().calendar()
    .buildRequest()
    .get();

```