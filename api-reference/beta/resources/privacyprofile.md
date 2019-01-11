---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
localization_priority: Normal
ms.openlocfilehash: adbd2e04e4d3898de559682b0b87158f938e7252
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833045"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="0ca3e-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ca3e-103">privacyProfile resource type</span></span>

> <span data-ttu-id="0ca3e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ca3e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ca3e-106">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-106">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="0ca3e-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ca3e-107">Properties</span></span>
| <span data-ttu-id="0ca3e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ca3e-108">Property</span></span>   | <span data-ttu-id="0ca3e-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ca3e-109">Type</span></span>|<span data-ttu-id="0ca3e-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ca3e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ca3e-111">contactEmail</span><span class="sxs-lookup"><span data-stu-id="0ca3e-111">contactEmail</span></span>|<span data-ttu-id="0ca3e-112">String</span><span class="sxs-lookup"><span data-stu-id="0ca3e-112">String</span></span>| <span data-ttu-id="0ca3e-113">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-113">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="0ca3e-114">可选。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-114">Not required.</span></span>|
|<span data-ttu-id="0ca3e-115">statementUrl</span><span class="sxs-lookup"><span data-stu-id="0ca3e-115">statementUrl</span></span>|<span data-ttu-id="0ca3e-116">String</span><span class="sxs-lookup"><span data-stu-id="0ca3e-116">String</span></span>| <span data-ttu-id="0ca3e-117">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-117">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="0ca3e-118">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-118">Maximum length is 255 characters.</span></span> <span data-ttu-id="0ca3e-119">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-119">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="0ca3e-120">可选。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-120">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ca3e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ca3e-121">JSON representation</span></span>

<span data-ttu-id="0ca3e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ca3e-122">Here is a JSON representation of the resource</span></span>

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
