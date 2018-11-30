---
title: mfaDetail 资源类型
description: '指示 MFA 特定登录的详细信息。 它包括用于登录以及身份验证的详细信息的身份验证方法 (例如： 电话、 SMS 或语音邮件) '
ms.openlocfilehash: a377c8648ebc8a6e3eb10fb6b0b87df066f8f2cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044751"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="cc910-104">mfaDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc910-104">mfaDetail resource type</span></span>
<span data-ttu-id="cc910-105">指示 MFA 特定登录的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cc910-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="cc910-106">它包括用于登录以及身份验证的详细信息的身份验证方法 (例如： 电话、 SMS 或语音邮件)</span><span class="sxs-lookup"><span data-stu-id="cc910-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="cc910-107">属性</span><span class="sxs-lookup"><span data-stu-id="cc910-107">Properties</span></span>
| <span data-ttu-id="cc910-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc910-108">Property</span></span>     | <span data-ttu-id="cc910-109">类型</span><span class="sxs-lookup"><span data-stu-id="cc910-109">Type</span></span>   |<span data-ttu-id="cc910-110">说明</span><span class="sxs-lookup"><span data-stu-id="cc910-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc910-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="cc910-111">authDetail</span></span>|<span data-ttu-id="cc910-112">字符串</span><span class="sxs-lookup"><span data-stu-id="cc910-112">String</span></span>|<span data-ttu-id="cc910-113">指示相应的登录活动的 MFA 身份验证的详细的信息时所需 MFA 为"Yes"。</span><span class="sxs-lookup"><span data-stu-id="cc910-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="cc910-114">身份验证方法</span><span class="sxs-lookup"><span data-stu-id="cc910-114">authMethod</span></span>|<span data-ttu-id="cc910-115">字符串</span><span class="sxs-lookup"><span data-stu-id="cc910-115">String</span></span>|<span data-ttu-id="cc910-116">所需的 MFA 字段为"Yes"时对相应的登录活动，指示 MFA 身份验证方法 （SMS、 电话、 Authenticator 应用程序是一些值的）。</span><span class="sxs-lookup"><span data-stu-id="cc910-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc910-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc910-117">JSON representation</span></span>

<span data-ttu-id="cc910-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc910-118">Here is a JSON representation of the resource.</span></span>

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