---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea90417d9b3ed77b136dac9f82f97cd43f9ea7fa1cb208083d7929973efa62cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSet reviewSet = graphClient.compliance().ediscovery().cases("6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d").reviewSets("0157910c-57ce-4e48-bd4b-90f3c88ca32e")
    .buildRequest()
    .get();

```