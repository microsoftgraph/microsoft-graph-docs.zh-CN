---
title: mfaDetail 资源类型
description: '指示特定登录的 MFA 详细信息。 它包括用于登录的身份验证方法以及身份验证的详细信息 (例如: 电话、短信或语音邮件) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3f38fae4d0360386592f956bee05d55738ad6910
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009662"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="21e56-104">mfaDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="21e56-104">mfaDetail resource type</span></span>
<span data-ttu-id="21e56-105">指示特定登录的 MFA 详细信息。</span><span class="sxs-lookup"><span data-stu-id="21e56-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="21e56-106">它包括用于登录的身份验证方法以及身份验证的详细信息 (例如: 电话、短信或语音邮件)</span><span class="sxs-lookup"><span data-stu-id="21e56-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="21e56-107">属性</span><span class="sxs-lookup"><span data-stu-id="21e56-107">Properties</span></span>
| <span data-ttu-id="21e56-108">属性</span><span class="sxs-lookup"><span data-stu-id="21e56-108">Property</span></span>     | <span data-ttu-id="21e56-109">类型</span><span class="sxs-lookup"><span data-stu-id="21e56-109">Type</span></span>   |<span data-ttu-id="21e56-110">说明</span><span class="sxs-lookup"><span data-stu-id="21e56-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21e56-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="21e56-111">authDetail</span></span>|<span data-ttu-id="21e56-112">String</span><span class="sxs-lookup"><span data-stu-id="21e56-112">String</span></span>|<span data-ttu-id="21e56-113">当所需的 MFA 为 "是" 时, 指示对应登录活动的 MFA 身份验证详细信息。</span><span class="sxs-lookup"><span data-stu-id="21e56-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="21e56-114">authMethod</span><span class="sxs-lookup"><span data-stu-id="21e56-114">authMethod</span></span>|<span data-ttu-id="21e56-115">String</span><span class="sxs-lookup"><span data-stu-id="21e56-115">String</span></span>|<span data-ttu-id="21e56-116">指示当 "MFA 必需" 字段为 "是" 时, 对相应登录活动的 MFA 身份验证方法 (SMS、电话、验证器应用程序值)。</span><span class="sxs-lookup"><span data-stu-id="21e56-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21e56-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21e56-117">JSON representation</span></span>

<span data-ttu-id="21e56-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21e56-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
