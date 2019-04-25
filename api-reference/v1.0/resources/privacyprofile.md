---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
ms.openlocfilehash: 29c4a01cde0e05c42ce74576e769ca005840e854
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579879"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="88fa9-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="88fa9-103">privacyProfile resource type</span></span>

<span data-ttu-id="88fa9-104">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="88fa9-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="88fa9-105">属性</span><span class="sxs-lookup"><span data-stu-id="88fa9-105">Properties</span></span>
| <span data-ttu-id="88fa9-106">属性</span><span class="sxs-lookup"><span data-stu-id="88fa9-106">Property</span></span>   | <span data-ttu-id="88fa9-107">类型</span><span class="sxs-lookup"><span data-stu-id="88fa9-107">Type</span></span>|<span data-ttu-id="88fa9-108">说明</span><span class="sxs-lookup"><span data-stu-id="88fa9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88fa9-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="88fa9-109">contactEmail</span></span>|<span data-ttu-id="88fa9-110">String</span><span class="sxs-lookup"><span data-stu-id="88fa9-110">String</span></span>| <span data-ttu-id="88fa9-111">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="88fa9-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="88fa9-112">可选。</span><span class="sxs-lookup"><span data-stu-id="88fa9-112">Not required.</span></span>|
|<span data-ttu-id="88fa9-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="88fa9-113">statementUrl</span></span>|<span data-ttu-id="88fa9-114">String</span><span class="sxs-lookup"><span data-stu-id="88fa9-114">String</span></span>| <span data-ttu-id="88fa9-115">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="88fa9-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="88fa9-116">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="88fa9-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="88fa9-117">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="88fa9-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="88fa9-118">可选。</span><span class="sxs-lookup"><span data-stu-id="88fa9-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88fa9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88fa9-119">JSON representation</span></span>

<span data-ttu-id="88fa9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88fa9-120">Here is a JSON representation of the resource</span></span>

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
