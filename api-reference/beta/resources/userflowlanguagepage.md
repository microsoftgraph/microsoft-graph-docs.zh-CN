---
title: userFlowLanguagePage 资源类型
description: 使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 25fb1c94db9443ed67a0555d09f3859e666bed19
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155466"
---
# <a name="userflowlanguagepage-resource-type"></a><span data-ttu-id="15afc-103">userFlowLanguagePage 资源类型</span><span class="sxs-lookup"><span data-stu-id="15afc-103">userFlowLanguagePage resource type</span></span>

<span data-ttu-id="15afc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15afc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15afc-105">使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。</span><span class="sxs-lookup"><span data-stu-id="15afc-105">User flow language pages are used determine the strings users will be shown during the user journey you have configured using user flows.</span></span> <span data-ttu-id="15afc-106">这些语言页面包括 Microsoft 提供的默认语言翻译或可创建自定义页面以自定义语言翻译。</span><span class="sxs-lookup"><span data-stu-id="15afc-106">These language pages include both the default language translations provided by Microsoft, or custom pages that can be created to customize the language translations.</span></span>

## <a name="methods"></a><span data-ttu-id="15afc-107">方法</span><span class="sxs-lookup"><span data-stu-id="15afc-107">Methods</span></span>

|<span data-ttu-id="15afc-108">方法</span><span class="sxs-lookup"><span data-stu-id="15afc-108">Method</span></span>|<span data-ttu-id="15afc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="15afc-109">Return type</span></span>|<span data-ttu-id="15afc-110">说明</span><span class="sxs-lookup"><span data-stu-id="15afc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15afc-111">获取 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="15afc-111">Get userFlowLanguagePage</span></span>](../api/userflowlanguagepage-get.md)|[<span data-ttu-id="15afc-112">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="15afc-112">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="15afc-113">检索默认或自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="15afc-113">Retrieve the values of a default or custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="15afc-114">更新 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="15afc-114">Update userFlowLanguagePage</span></span>](../api/userflowlanguagepage-put.md)|[<span data-ttu-id="15afc-115">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="15afc-115">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="15afc-116">更新自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 中的值。</span><span class="sxs-lookup"><span data-stu-id="15afc-116">Update the values in a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="15afc-117">删除 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="15afc-117">Delete userFlowLanguagePage</span></span>](../api/userflowlanguagepage-delete.md)|<span data-ttu-id="15afc-118">无</span><span class="sxs-lookup"><span data-stu-id="15afc-118">None</span></span>|<span data-ttu-id="15afc-119">从自定义 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中删除值。</span><span class="sxs-lookup"><span data-stu-id="15afc-119">Deletes the values from a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15afc-120">属性</span><span class="sxs-lookup"><span data-stu-id="15afc-120">Properties</span></span>

|<span data-ttu-id="15afc-121">属性</span><span class="sxs-lookup"><span data-stu-id="15afc-121">Property</span></span>|<span data-ttu-id="15afc-122">类型</span><span class="sxs-lookup"><span data-stu-id="15afc-122">Type</span></span>|<span data-ttu-id="15afc-123">说明</span><span class="sxs-lookup"><span data-stu-id="15afc-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15afc-124">id</span><span class="sxs-lookup"><span data-stu-id="15afc-124">id</span></span>|<span data-ttu-id="15afc-125">String</span><span class="sxs-lookup"><span data-stu-id="15afc-125">String</span></span>|<span data-ttu-id="15afc-126">userFlowLanguage 页的标识符。</span><span class="sxs-lookup"><span data-stu-id="15afc-126">The identifier of the userFlowLanguage page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15afc-127">关系</span><span class="sxs-lookup"><span data-stu-id="15afc-127">Relationships</span></span>

<span data-ttu-id="15afc-128">无。</span><span class="sxs-lookup"><span data-stu-id="15afc-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15afc-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15afc-129">JSON representation</span></span>

<span data-ttu-id="15afc-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15afc-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
