---
title: insightIdentity
description: " 资源类型"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046081"
---
# <a name="insightidentity"></a>insightIdentity

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

 资源类型

包含[共享](insights-shared.md)项目的属性的复杂类型。 

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |-----------    | -------------|
| displayName       | 字符串          | 共享项目的用户的显示名称。 |
| id              | 字符串        | 共享项目的用户的 id。     |
| address             | String      | 共享项目的用户的电子邮件地址。  |