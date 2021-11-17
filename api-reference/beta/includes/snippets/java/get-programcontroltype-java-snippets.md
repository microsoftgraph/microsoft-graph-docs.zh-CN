---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c508f3026a954d3b493a125e2ff21a56cd56b0d44ac26375958c2fdaaa7ede6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221074"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControlTypeCollectionPage programControlTypes = graphClient.programControlTypes()
    .buildRequest()
    .get();

```