---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a64defb220a6c8adc28ba06cd205c1eb70496329
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469428"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="63d55-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="63d55-103">privacyProfile resource type</span></span>

<span data-ttu-id="63d55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63d55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63d55-105">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="63d55-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="63d55-106">属性</span><span class="sxs-lookup"><span data-stu-id="63d55-106">Properties</span></span>
| <span data-ttu-id="63d55-107">属性</span><span class="sxs-lookup"><span data-stu-id="63d55-107">Property</span></span>   | <span data-ttu-id="63d55-108">类型</span><span class="sxs-lookup"><span data-stu-id="63d55-108">Type</span></span>|<span data-ttu-id="63d55-109">说明</span><span class="sxs-lookup"><span data-stu-id="63d55-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63d55-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="63d55-110">contactEmail</span></span>|<span data-ttu-id="63d55-111">String</span><span class="sxs-lookup"><span data-stu-id="63d55-111">String</span></span>| <span data-ttu-id="63d55-112">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="63d55-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="63d55-113">可选。</span><span class="sxs-lookup"><span data-stu-id="63d55-113">Not required.</span></span>|
|<span data-ttu-id="63d55-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="63d55-114">statementUrl</span></span>|<span data-ttu-id="63d55-115">String</span><span class="sxs-lookup"><span data-stu-id="63d55-115">String</span></span>| <span data-ttu-id="63d55-116">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="63d55-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="63d55-117">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="63d55-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="63d55-118">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="63d55-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="63d55-119">可选。</span><span class="sxs-lookup"><span data-stu-id="63d55-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63d55-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63d55-120">JSON representation</span></span>

<span data-ttu-id="63d55-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63d55-121">Here is a JSON representation of the resource</span></span>

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

