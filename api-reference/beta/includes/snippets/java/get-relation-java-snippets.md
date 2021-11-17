---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a14ff42f94374beb27c828c333f44944dd682020168fcddf2735931208798bc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279617"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RelationCollectionPage relations = graphClient.termStore().sets("{setId}").relations()
    .buildRequest()
    .get();

```