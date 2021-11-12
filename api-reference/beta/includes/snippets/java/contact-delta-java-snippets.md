---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c21122f9f7710d2c6e0dd933e122aced6cceb85933799a5de1fd4ca4f4f10365
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274196"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactDeltaCollectionPage delta = graphClient.me().contactFolders("{id}").contacts()
    .delta()
    .buildRequest()
    .select("displayName")
    .get();

```