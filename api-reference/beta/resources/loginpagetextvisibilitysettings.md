---
title: loginPageTextVisibilitySettings 资源类型
description: 包含组织品牌打造的详细信息。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f31973dad83f09305bdae6a9f9997b6af35d5049
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805430"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>loginPageTextVisibilitySettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

这是一个复杂类型，表示可在租户的登录页面上隐藏的各种文本。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| hideCannotAccessYourAccount | 布尔值 | 用于隐藏 SSPR 帐户的自助服务密码重置 (选项) 无法访问您的帐户？" 超链接。 |
| hideForgotMyPassword | 布尔值 | 在登录表单上隐藏 SSPR (密码重置) "忘记密码"超链接的选项。 |
| hideResetItNow | 布尔值 | 用于隐藏登录表单上 SSPR (密码重置) "立即重置"超链接的选项。 |
| hideTermsOfUse | 布尔值 | 用于隐藏页脚中的"使用条款"超链接的选项。 |
| hidePrivacyAndCookies | 布尔值 | 用于隐藏页脚中的"& Cookie"超链接的选项。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loginPageTextVisibilitySettings",
  "hideCannotAccessYourAccount": "Boolean",
  "hideForgotMyPassword": "Boolean",
  "hidePrivacyAndCookies": "Boolean",
  "hideResetItNow": "Boolean",
  "hideTermsOfUse": "Boolean"
}
```
