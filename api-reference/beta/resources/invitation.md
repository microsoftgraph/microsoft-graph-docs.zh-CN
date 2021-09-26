---
title: 邀请资源类型
description: 表示用于将外部用户添加到组织的邀请。
ms.localizationpriority: medium
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6998b38dc51af04d5f7314a52663fa2b9b5cccb2
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766353"
---
# <a name="invitation-resource-type"></a>邀请资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于将外部用户添加到组织的邀请。 

邀请进程使用以下流程：

* 创建邀请
* 将邀请发送至邀请的用户（包含邀请链接）
* 邀请的用户单击邀请链接、登录并兑现邀请和创建用户实体表示邀请的用户完成操作
* 兑现完成后，将用户重定向至指定页面

创建邀请会在响应中返回兑现 URL (*inviteRedeemUrl*)。通过将 *sendInvitationMessage* 设置为 true，创建邀请 API 可以自动向邀请的用户发送包含兑现 URL 的电子邮件。还可以自定义要发送至邀请的用户的邮件。反之，如果想要通过一些其他的方法发送兑现 URL，则可以将 *sendInvitationMessage* 设置为 false，然后使用响应中的兑现 URL 创建自己的通信。目前没有可以执行兑现进程的 API。邀请的用户必须单击在上述步骤中的通信中发送的 *inviteRedeemUrl* 链接，并在浏览器中进行交互式兑现流程。完成后，邀请的用户即成为组织中的外部用户。

>[!NOTE]
>使用作为邀请请求的一部分创建的外部用户资源上的 [](user.md)**externalUserState** 和 **externalUserStateChangeDateTime** 属性跟踪邀请状态。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建邀请](../api/invitation-post.md) | 邀请 | 写入 invitation 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|invitedUserDisplayName|String|被邀请的用户的显示名称。|
|invitedUserEmailAddress|String|被邀请的用户的电子邮件地址。 必需。 电子邮件地址中不允许使用以下特殊字符：<br><ul><li>波形符 (~)</li><li>感叹号 (`!`)</li><li>@ 符号 (`@`)</li><li>井号 (`#`)</li><li>美元符号 (`$`)</li><li>百分号 (`%`)</li><li>扬抑符 (`^`)</li><li>与号 (`&`)</li><li>星号 (`*`)</li><li>圆括号 (`( )`)</li><li>连字符 (`-`)</li><li>加号 (`+`)</li><li>等号 (`=`)</li><li>方括号 (`[ ]`)</li><li>大括号 (`{ }`)</li><li>反斜杠 (`\`)</li><li>斜杠符号 (`/`)</li><li>竖线 (`|`)</li><li>分号 (`;`)</li><li>冒号 (`:`)</li><li>引号 (`"`)</li><li>尖括号 (`< >`)</li><li>问号 (`?`)</li><li>逗号 (`,`)</li></ul><br>但是，存在下列例外情况：<br><ul><li>允许在用户名中的任何位置使用句点 (`.`) 或连字符 (`-`)，但名称的开头或结尾除外。</li><li>允许在用户名中的任何位置使用下划线 (`_`)。 这包括名称的开头或结尾。</li></ul>|
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|要发送至邀请用户的邮件的其他配置，其中包括自定义邮件文本、语言和抄送收件人列表。|
|inviteRedirectUrl|String|兑现邀请后，用户应被重定向至的 URL。必填。|
|inviteRedeemUrl|String|用户用于兑现邀请的 URL。只读。|
|invitedUserType|String|被邀请的用户的 userType。 默认情况下，此操作为 `Guest`。 你可以像 `Member` 你是公司管理员一样进行邀请。 默认值为 `false`。 |
|resetRedemption|Boolean|重置用户的兑换状态并重新邀请用户，同时保留其用户标识符、组成员身份以及应用分配。 此属性允许用户使用与上一邀请中的电子邮件地址不同的电子邮件地址登录。 有关使用此属性的详细信息，请参阅重置来宾用户的兑换状态 ([预览) 。 ](/azure/active-directory/external-identities/reset-redemption-status#use-microsoft-graph-api-to-reset-redemption-status)|
|sendInvitationMessage|Boolean|指示电子邮件是否应发送至邀请的用户。 默认值为 `false`。|
|status|String|邀请的状态。 可能的值 `PendingAcceptance` `Completed` ：、、 `InProgress` 和 `Error`|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|invitedUser|[user](user.md)|创建为邀请创建进程组成部分的用户。只读|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- 
{ 
    "blockType": "resource",
    "keyProperty":"id",
    "@odata.type": "microsoft.graph.invitation", 
    "optionalProperties": [
        "invitedUser"
     ],
    "baseType": "microsoft.graph.entity"
} 
-->
```json
{
  "id": "String",
  "invitedUserDisplayName": "String",
  "invitedUserEmailAddress": "String",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "String",
  "inviteRedeemUrl": "String",
  "resetRedemption": false,
  "status": "String",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "String"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


