---
title: 使用员工学习 API 与Viva Learning集成
description: 了解如何注册提供程序，以及如何将学习提供程序中的内容和学习器记录集成到Viva Learning。
ms.localizationpriority: medium
author: malabikaroy
ms.prod: employee-learning
doc_type: conceptualPageType
ms.openlocfilehash: f8112d21cc4d3677c4b36398539a529c247ecd39
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883280"
---
# <a name="use-the-employee-learning-api-to-integrate-with-viva-learning"></a>使用员工学习 API 与Viva Learning集成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Viva Learning是 Microsoft Teams 中的一个集中式员工学习中心，使员工能够将学习和生成技能集成到工作日。 在Viva Learning中，团队可以发现、共享、推荐和学习其组织和合作伙伴提供的内容库。 他们可以快速访问分配或最近完成的学习内容，并在不离开 Microsoft Teams 的情况下执行所有这些操作。

通过 Microsoft Graph 中的员工学习 API，应用可以使学习管理系统 (LMS) 或学习提供程序中的内容在Viva Learning中可用。 使用以下资源与Viva Learning集成：

- 用于管理学习提供程序的[学习提供](learningprovider.md)程序，包括注册、启用、禁用或删除提供程序。
- [在](learningcontent.md)Viva Learning中学习要从 LMS 或学习提供程序上传和管理学习内容元数据的内容。


## <a name="how-do-integrations-work"></a>集成的工作原理是什么？
作为管理员，可以使用现成的集成，将内容和学习器记录 (员工分配和已完成的课程记录) LMS 或学习提供程序与Viva Learning集成，其中Viva Learning可以从 LMS 或学习提供程序提取内容元数据和学习记录。 还可以使用 Microsoft Graph 中[的员工学习 API](#use-cases-for-the-employee-learning-api-in-microsoft-graph) 将内容元数据从 LMS 或学习提供程序推送到Viva Learning。 

将内容元数据、员工分配及其已完成的课程记录上传到Viva Learning时，它们将显示在以下位置的Viva Learning中：
- 内容显示在“ **浏览课程** - **提供程序** ”部分下的主页上。
- 作业和已完成的课程记录分别显示在 **“分配给你**”和“**已完成**”部分下的“**我的学习**”页上。

## <a name="authorization"></a>Authorization
使用适当的委派或应用程序 [员工学习权限](/graph/permissions-reference#employee-learning-permissions)，你的应用可以使用员工学习 API 管理租户中学习中心的学习提供程序及其内容。 有关访问令牌、应用注册以及委派和应用程序权限的详细信息，请参阅 [身份验证和授权基础知识](/graph/auth/auth-concepts)。

## <a name="use-cases-for-the-employee-learning-api-in-microsoft-graph"></a>Microsoft Graph 中员工学习 API 的用例
使用员工学习 API 执行以下操作：
- [向Viva Learning注册提供程序](../api/employeeexperience-post-learningproviders.md)，提供显示名称、在学习内容卡上显示的方形徽标，以及“**详细信息**”页中显示的长徽标，提供程序内容需要显示在Viva Learning中。 返回的注册 ID 可用于对内容引入进行后续调用。
- 启用或禁用注册并更新提供程序的显示名称和徽标 URL。  
- [获取特定 registrationId Viva Learning中的提供程序的详细信息](../api/learningprovider-get.md)。  
- [获取租户Viva Learning中的提供程序注册列表](../api/employeeexperience-list-learningproviders.md)。
- [在](../api/employeeexperience-delete-learningproviders.md)Viva Learning中删除提供程序的注册。
- [将内容元数据推](../api/learningcontent-update.md)送到Viva Learning，使内容在Viva Learning中可用，供用户使用。  
- 使用提供程序的 **registrationId** [获取提供程序引入内容的元数据列表](../api/learningprovider-list-learningcontents.md)。  
- [获取提供程序在Viva Learning中引入的内容的指定元](../api/learningcontent-get.md)数据。
- [删除提供程序引入内容的指定元数据](../api/learningprovider-delete-learningcontents.md)。

>**注意**：员工学习 API 中尚不可用分配和已完成的课程记录。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤
- [使用 Teams 中的协作功能启用员工学习](/graph/teams-concept-overview#enable-employee-learning-using-the-collaborative-capabilities-in-teams)。
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用员工学习 API。
