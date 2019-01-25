---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510118"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="73efe-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="73efe-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73efe-104">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="73efe-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="73efe-105">属性</span><span class="sxs-lookup"><span data-stu-id="73efe-105">Properties</span></span>
| <span data-ttu-id="73efe-106">属性</span><span class="sxs-lookup"><span data-stu-id="73efe-106">Property</span></span>   | <span data-ttu-id="73efe-107">类型</span><span class="sxs-lookup"><span data-stu-id="73efe-107">Type</span></span>|<span data-ttu-id="73efe-108">说明</span><span class="sxs-lookup"><span data-stu-id="73efe-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73efe-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="73efe-109">contactEmail</span></span>|<span data-ttu-id="73efe-110">String</span><span class="sxs-lookup"><span data-stu-id="73efe-110">String</span></span>| <span data-ttu-id="73efe-111">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="73efe-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="73efe-112">可选。</span><span class="sxs-lookup"><span data-stu-id="73efe-112">Not required.</span></span>|
|<span data-ttu-id="73efe-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="73efe-113">statementUrl</span></span>|<span data-ttu-id="73efe-114">String</span><span class="sxs-lookup"><span data-stu-id="73efe-114">String</span></span>| <span data-ttu-id="73efe-115">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="73efe-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="73efe-116">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="73efe-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="73efe-117">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="73efe-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="73efe-118">可选。</span><span class="sxs-lookup"><span data-stu-id="73efe-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73efe-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73efe-119">JSON representation</span></span>

<span data-ttu-id="73efe-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73efe-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/privacyprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
