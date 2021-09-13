---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dd99ce406323f0e98536bdbc49a8f3578610924924fb2aa0e4dd7f67118b743
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221002"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8")
    .publish()
    .buildRequest()
    .post();

```