---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cadd430fe6f03d9d5d1800fcaf474bc5723e8e6b2fb271a02ef3a57a258e835
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332348"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCollectionPage people = graphClient.me().people()
    .buildRequest()
    .get();

```