---
title: userFlowLanguagePage 资源类型
description: 使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6a6bd597fb274d8fdb8150be0a2c5e085949156
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706244"
---
# <a name="userflowlanguagepage-resource-type"></a><span data-ttu-id="330ae-103">userFlowLanguagePage 资源类型</span><span class="sxs-lookup"><span data-stu-id="330ae-103">userFlowLanguagePage resource type</span></span>

<span data-ttu-id="330ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="330ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="330ae-105">使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。</span><span class="sxs-lookup"><span data-stu-id="330ae-105">User flow language pages are used determine the strings users will be shown during the user journey you have configured using user flows.</span></span> <span data-ttu-id="330ae-106">这些语言页面包括 Microsoft 提供的默认语言翻译，或可创建自定义语言翻译的自定义页面。</span><span class="sxs-lookup"><span data-stu-id="330ae-106">These language pages include both the default language translations provided by Microsoft, or custom pages that can be created to customize the language translations.</span></span>

## <a name="methods"></a><span data-ttu-id="330ae-107">方法</span><span class="sxs-lookup"><span data-stu-id="330ae-107">Methods</span></span>

|<span data-ttu-id="330ae-108">方法</span><span class="sxs-lookup"><span data-stu-id="330ae-108">Method</span></span>|<span data-ttu-id="330ae-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="330ae-109">Return type</span></span>|<span data-ttu-id="330ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="330ae-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="330ae-111">获取 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="330ae-111">Get userFlowLanguagePage</span></span>](../api/userflowlanguagepage-get.md)|[<span data-ttu-id="330ae-112">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="330ae-112">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="330ae-113">检索默认或自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="330ae-113">Retrieve the values of a default or custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="330ae-114">更新 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="330ae-114">Update userFlowLanguagePage</span></span>](../api/userflowlanguagepage-put.md)|[<span data-ttu-id="330ae-115">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="330ae-115">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="330ae-116">更新自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 中的值。</span><span class="sxs-lookup"><span data-stu-id="330ae-116">Update the values in a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="330ae-117">删除 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="330ae-117">Delete userFlowLanguagePage</span></span>](../api/userflowlanguagepage-delete.md)|<span data-ttu-id="330ae-118">无</span><span class="sxs-lookup"><span data-stu-id="330ae-118">None</span></span>|<span data-ttu-id="330ae-119">从自定义 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中删除值。</span><span class="sxs-lookup"><span data-stu-id="330ae-119">Deletes the values from a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="330ae-120">属性</span><span class="sxs-lookup"><span data-stu-id="330ae-120">Properties</span></span>

|<span data-ttu-id="330ae-121">属性</span><span class="sxs-lookup"><span data-stu-id="330ae-121">Property</span></span>|<span data-ttu-id="330ae-122">类型</span><span class="sxs-lookup"><span data-stu-id="330ae-122">Type</span></span>|<span data-ttu-id="330ae-123">说明</span><span class="sxs-lookup"><span data-stu-id="330ae-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="330ae-124">id</span><span class="sxs-lookup"><span data-stu-id="330ae-124">id</span></span>|<span data-ttu-id="330ae-125">字符串</span><span class="sxs-lookup"><span data-stu-id="330ae-125">String</span></span>|<span data-ttu-id="330ae-126">userFlowLanguage 页的标识符。</span><span class="sxs-lookup"><span data-stu-id="330ae-126">The identifier of the userFlowLanguage page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="330ae-127">关系</span><span class="sxs-lookup"><span data-stu-id="330ae-127">Relationships</span></span>

<span data-ttu-id="330ae-128">无。</span><span class="sxs-lookup"><span data-stu-id="330ae-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="330ae-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="330ae-129">JSON representation</span></span>

<span data-ttu-id="330ae-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="330ae-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
