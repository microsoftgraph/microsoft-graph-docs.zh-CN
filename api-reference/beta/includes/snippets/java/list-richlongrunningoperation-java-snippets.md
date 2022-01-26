---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e639b837bd16b2ca86798d890f2f4e6e1ca17cba
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225899"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RichLongRunningOperationCollectionPage operations = graphClient.sites("{site-ID}").operations()
    .buildRequest()
    .get();

```