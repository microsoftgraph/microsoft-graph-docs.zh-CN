---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e43064fe520f100d582e740302a7606c9824b3f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521563"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="8dcd0-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="8dcd0-103">privacyProfile resource type</span></span>

<span data-ttu-id="8dcd0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8dcd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dcd0-105">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="8dcd0-106">属性</span><span class="sxs-lookup"><span data-stu-id="8dcd0-106">Properties</span></span>
| <span data-ttu-id="8dcd0-107">属性</span><span class="sxs-lookup"><span data-stu-id="8dcd0-107">Property</span></span>   | <span data-ttu-id="8dcd0-108">类型</span><span class="sxs-lookup"><span data-stu-id="8dcd0-108">Type</span></span>|<span data-ttu-id="8dcd0-109">说明</span><span class="sxs-lookup"><span data-stu-id="8dcd0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dcd0-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="8dcd0-110">contactEmail</span></span>|<span data-ttu-id="8dcd0-111">String</span><span class="sxs-lookup"><span data-stu-id="8dcd0-111">String</span></span>| <span data-ttu-id="8dcd0-112">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="8dcd0-113">可选。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-113">Not required.</span></span>|
|<span data-ttu-id="8dcd0-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="8dcd0-114">statementUrl</span></span>|<span data-ttu-id="8dcd0-115">String</span><span class="sxs-lookup"><span data-stu-id="8dcd0-115">String</span></span>| <span data-ttu-id="8dcd0-116">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="8dcd0-117">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="8dcd0-118">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="8dcd0-119">可选。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dcd0-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8dcd0-120">JSON representation</span></span>

<span data-ttu-id="8dcd0-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dcd0-121">Here is a JSON representation of the resource</span></span>

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
