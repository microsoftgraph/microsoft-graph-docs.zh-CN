---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c3867aa9d91441b72964d3c5813d6db21abb6d18218fd13719c50e3c3da1db7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218573"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .close()
    .buildRequest()
    .post();

```