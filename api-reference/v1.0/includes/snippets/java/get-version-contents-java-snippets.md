---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 446acf84304de6cda60259fd4702f179f72c5ce94760ffd20019d83996c3e005
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219658"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/drive/items/{item-id}/versions/{version-id}/content", InputStream.class)
    .buildRequest()
    .get();

```