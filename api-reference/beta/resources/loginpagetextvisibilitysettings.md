---
title: loginPageTextVisibilitySettings 资源类型
description: 包含组织的品牌的详细信息。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9a18a8678db335b788ef170f97958de5154a1942
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441718"
---
# <a name="loginpagetextvisibilitysettings-resource-type"></a>loginPageTextVisibilitySettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可在租户的登录页上隐藏的各种文本字符串。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| hideAccountResetCredentials | Boolean | 在 SSPR () 超链接（例如“无法访问帐户？”、“忘记我的密码”和“立即重置密码”）中隐藏自助密码重置的选项。 |
| hideCannotAccessYourAccount | Boolean |  (SSPR) “无法访问帐户？”隐藏自助密码重置的选项 登录窗体上的超链接。 |
| hideForgotMyPassword | Boolean | 在登录窗体上隐藏自助密码重置 (SSPR) “忘记我的密码”超链接的选项。 |
| hideResetItNow | Boolean | 在登录窗体上隐藏自助密码重置 (SSPR) “立即重置”超链接的选项。 |
| hideTermsOfUse | Boolean | 在页脚中隐藏“使用条款”超链接的选项。 |
| hidePrivacyAndCookies | Boolean | 在页脚中隐藏“隐私& Cookie”超链接的选项。 |

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
  "hideAccountResetCredentials": "Boolean",
  "hideCannotAccessYourAccount": "Boolean",
  "hideForgotMyPassword": "Boolean",
  "hidePrivacyAndCookies": "Boolean",
  "hideResetItNow": "Boolean",
  "hideTermsOfUse": "Boolean"
}
```
