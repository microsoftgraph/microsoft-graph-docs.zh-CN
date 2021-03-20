---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b54fd15d5dc52a1c085bf3b5c743401d4101318f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971072"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CaseOperationCollectionPage operations = graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583").operations()
    .buildRequest()
    .get();

```