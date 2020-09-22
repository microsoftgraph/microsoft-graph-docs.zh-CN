---
title: educationPowerSchoolDataProvider 资源
description: 用于在将 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 664b7c9c3ad255e502583fca6be332043e712a46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979614"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="4c257-103">educationPowerSchoolDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="4c257-103">educationPowerSchoolDataProvider resource</span></span>

<span data-ttu-id="4c257-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c257-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c257-105">用于在将 [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) 用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="4c257-105">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="4c257-106">派生自 [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="4c257-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4c257-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c257-107">Properties</span></span>

| <span data-ttu-id="4c257-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c257-108">Property</span></span>                       | <span data-ttu-id="4c257-109">类型</span><span class="sxs-lookup"><span data-stu-id="4c257-109">Type</span></span>                                     | <span data-ttu-id="4c257-110">说明</span><span class="sxs-lookup"><span data-stu-id="4c257-110">Description</span></span>                                                                            |
| :----------------------------- | :--------------------------------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="4c257-111">allowTeachersInMultipleSchools</span><span class="sxs-lookup"><span data-stu-id="4c257-111">allowTeachersInMultipleSchools</span></span> | <span data-ttu-id="4c257-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c257-112">Boolean</span></span>                                  | <span data-ttu-id="4c257-113">指示源是否具有单个学生或教师的多个标识符。</span><span class="sxs-lookup"><span data-stu-id="4c257-113">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="4c257-114">clientId</span><span class="sxs-lookup"><span data-stu-id="4c257-114">clientId</span></span>                       | <span data-ttu-id="4c257-115">字符串</span><span class="sxs-lookup"><span data-stu-id="4c257-115">String</span></span>                                   | <span data-ttu-id="4c257-116">用于连接到 PowerSchool 的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="4c257-116">The client ID used to connect to PowerSchool.</span></span>                                          |
| <span data-ttu-id="4c257-117">clientSecret</span><span class="sxs-lookup"><span data-stu-id="4c257-117">clientSecret</span></span>                   | <span data-ttu-id="4c257-118">字符串</span><span class="sxs-lookup"><span data-stu-id="4c257-118">String</span></span>                                   | <span data-ttu-id="4c257-119">用于对与 PowerSchool 实例的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="4c257-119">The client secret to authenticate the connection to the PowerSchool instance.</span></span>          |
| <span data-ttu-id="4c257-120">connectionUrl</span><span class="sxs-lookup"><span data-stu-id="4c257-120">connectionUrl</span></span>                  | <span data-ttu-id="4c257-121">String</span><span class="sxs-lookup"><span data-stu-id="4c257-121">String</span></span>                                   | <span data-ttu-id="4c257-122">指向 PowerSchool 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="4c257-122">The connection URL to the PowerSchool instance.</span></span>                                        |
| <span data-ttu-id="4c257-123">schoolsIds</span><span class="sxs-lookup"><span data-stu-id="4c257-123">schoolsIds</span></span>                     | <span data-ttu-id="4c257-124">String collection</span><span class="sxs-lookup"><span data-stu-id="4c257-124">String collection</span></span>                        | <span data-ttu-id="4c257-125">要同步的学校列表。</span><span class="sxs-lookup"><span data-stu-id="4c257-125">The list of schools to sync.</span></span>                                                           |
| <span data-ttu-id="4c257-126">schoolYear</span><span class="sxs-lookup"><span data-stu-id="4c257-126">schoolYear</span></span>                     | <span data-ttu-id="4c257-127">String</span><span class="sxs-lookup"><span data-stu-id="4c257-127">String</span></span>                                   | <span data-ttu-id="4c257-128">要同步的学校年。</span><span class="sxs-lookup"><span data-stu-id="4c257-128">The school year to sync.</span></span>                                                               |
| <span data-ttu-id="4c257-129">操作</span><span class="sxs-lookup"><span data-stu-id="4c257-129">customizations</span></span>                 | <span data-ttu-id="4c257-130">[educationSynchronizationCustomizations]</span><span class="sxs-lookup"><span data-stu-id="4c257-130">[educationSynchronizationCustomizations]</span></span> | <span data-ttu-id="4c257-131">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="4c257-131">Optional customization to be applied to the synchronization profile.</span></span>                   |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a><span data-ttu-id="4c257-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c257-133">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```


