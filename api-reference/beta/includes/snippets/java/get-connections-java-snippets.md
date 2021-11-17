---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd0a466d7f15461292337569a9e5ebe906412817faba1cfa9635d428c01119b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215849"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnectionCollectionPage connections = graphClient.external().connections()
    .buildRequest()
    .get();

```