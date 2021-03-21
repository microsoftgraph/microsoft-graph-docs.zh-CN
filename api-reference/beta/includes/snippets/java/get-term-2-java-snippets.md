---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f5d26cabe8b7f9b19bcdfe887ea8a6047b5083d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955371"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITermCollectionPage children = graphClient.termStore().sets("{setId}").children()
    .buildRequest()
    .get();

```