---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6503cf43016389860d5454b405602cfaa906b909e67bf4d84635c1a1b19f033
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161218"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LanguageProficiency languageProficiency = graphClient.me().profile().languages("{id}")
    .buildRequest()
    .get();

```