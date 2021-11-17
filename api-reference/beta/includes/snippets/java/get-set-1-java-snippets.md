---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c2b0a442136df535fb7ce541a980c53300643fef19cd10d427622994a970c5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SetCollectionPage sets = graphClient.termStore().groups("{groupId}").sets()
    .buildRequest()
    .get();

```