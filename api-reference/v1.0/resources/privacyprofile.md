---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ec7de45bdffc2a8a00ac6519afb55cfbbc841429
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811271"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="1b5cd-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b5cd-103">privacyProfile resource type</span></span>

<span data-ttu-id="1b5cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b5cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b5cd-105">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="1b5cd-106">属性</span><span class="sxs-lookup"><span data-stu-id="1b5cd-106">Properties</span></span>
| <span data-ttu-id="1b5cd-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b5cd-107">Property</span></span>   | <span data-ttu-id="1b5cd-108">类型</span><span class="sxs-lookup"><span data-stu-id="1b5cd-108">Type</span></span>|<span data-ttu-id="1b5cd-109">说明</span><span class="sxs-lookup"><span data-stu-id="1b5cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b5cd-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="1b5cd-110">contactEmail</span></span>|<span data-ttu-id="1b5cd-111">String</span><span class="sxs-lookup"><span data-stu-id="1b5cd-111">String</span></span>| <span data-ttu-id="1b5cd-112">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="1b5cd-113">可选。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-113">Not required.</span></span>|
|<span data-ttu-id="1b5cd-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="1b5cd-114">statementUrl</span></span>|<span data-ttu-id="1b5cd-115">String</span><span class="sxs-lookup"><span data-stu-id="1b5cd-115">String</span></span>| <span data-ttu-id="1b5cd-116">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="1b5cd-117">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="1b5cd-118">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="1b5cd-119">可选。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b5cd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b5cd-120">JSON representation</span></span>

<span data-ttu-id="1b5cd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b5cd-121">Here is a JSON representation of the resource</span></span>

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
