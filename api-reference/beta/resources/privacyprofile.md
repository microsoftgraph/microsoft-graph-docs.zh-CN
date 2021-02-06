---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 986f995458c56869d966c3c1baa2dc2f5df9aca1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137667"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="a7997-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7997-103">privacyProfile resource type</span></span>

<span data-ttu-id="a7997-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7997-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7997-105">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="a7997-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="a7997-106">属性</span><span class="sxs-lookup"><span data-stu-id="a7997-106">Properties</span></span>
| <span data-ttu-id="a7997-107">属性</span><span class="sxs-lookup"><span data-stu-id="a7997-107">Property</span></span>   | <span data-ttu-id="a7997-108">类型</span><span class="sxs-lookup"><span data-stu-id="a7997-108">Type</span></span>|<span data-ttu-id="a7997-109">说明</span><span class="sxs-lookup"><span data-stu-id="a7997-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7997-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="a7997-110">contactEmail</span></span>|<span data-ttu-id="a7997-111">String</span><span class="sxs-lookup"><span data-stu-id="a7997-111">String</span></span>| <span data-ttu-id="a7997-112">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a7997-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="a7997-113">可选。</span><span class="sxs-lookup"><span data-stu-id="a7997-113">Not required.</span></span>|
|<span data-ttu-id="a7997-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="a7997-114">statementUrl</span></span>|<span data-ttu-id="a7997-115">String</span><span class="sxs-lookup"><span data-stu-id="a7997-115">String</span></span>| <span data-ttu-id="a7997-116">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="a7997-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="a7997-117">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="a7997-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="a7997-118">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="a7997-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="a7997-119">可选。</span><span class="sxs-lookup"><span data-stu-id="a7997-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7997-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7997-120">JSON representation</span></span>

<span data-ttu-id="a7997-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7997-121">Here is a JSON representation of the resource</span></span>

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


