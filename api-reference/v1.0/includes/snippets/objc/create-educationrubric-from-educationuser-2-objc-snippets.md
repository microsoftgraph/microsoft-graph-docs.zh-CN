---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4e56ff7e9a8498ac65fffe2eaf275858ac7f2619b347f4c97f4824d621ca7f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332787"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/me/rubrics"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationRubric *educationRubric = [[MSGraphEducationRubric alloc] init];
[educationRubric setDisplayName:@"Example Points Rubric"];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"This is an example of a rubric with points"];
[description setContentType: [MSGraphBodyType text]];
[educationRubric setDescription:description];
NSMutableArray *levelsList = [[NSMutableArray alloc] init];
MSGraphRubricLevel *levels = [[MSGraphRubricLevel alloc] init];
[levels setDisplayName:@"Good"];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@""];
[description setContentType: [MSGraphBodyType text]];
[levels setDescription:description];
MSGraphEducationAssignmentGradeType *grading = [[MSGraphEducationAssignmentGradeType alloc] init];
[grading setMaxPoints: 2];
[levels setGrading:grading];
[levelsList addObject: levels];
MSGraphRubricLevel *levels = [[MSGraphRubricLevel alloc] init];
[levels setDisplayName:@"Poor"];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@""];
[description setContentType: [MSGraphBodyType text]];
[levels setDescription:description];
MSGraphEducationAssignmentGradeType *grading = [[MSGraphEducationAssignmentGradeType alloc] init];
[grading setMaxPoints: 1];
[levels setGrading:grading];
[levelsList addObject: levels];
[educationRubric setLevels:levelsList];
NSMutableArray *qualitiesList = [[NSMutableArray alloc] init];
MSGraphRubricQuality *qualities = [[MSGraphRubricQuality alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"Argument"];
[description setContentType: [MSGraphBodyType text]];
[qualities setDescription:description];
NSMutableArray *criteriaList = [[NSMutableArray alloc] init];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay's argument is persuasive."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay's argument does not make sense."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
[qualities setCriteria:criteriaList];
[qualities setWeight: 50.0];
[qualitiesList addObject: qualities];
MSGraphRubricQuality *qualities = [[MSGraphRubricQuality alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"Spelling and Grammar"];
[description setContentType: [MSGraphBodyType text]];
[qualities setDescription:description];
NSMutableArray *criteriaList = [[NSMutableArray alloc] init];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay uses proper spelling and grammar with few or no errors."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
MSGraphRubricCriterion *criteria = [[MSGraphRubricCriterion alloc] init];
MSGraphEducationItemBody *description = [[MSGraphEducationItemBody alloc] init];
[description setContent:@"The essay has numerous errors in spelling and/or grammar."];
[description setContentType: [MSGraphBodyType text]];
[criteria setDescription:description];
[criteriaList addObject: criteria];
[qualities setCriteria:criteriaList];
[qualities setWeight: 50.0];
[qualitiesList addObject: qualities];
[educationRubric setQualities:qualitiesList];
MSGraphEducationAssignmentGradeType *grading = [[MSGraphEducationAssignmentGradeType alloc] init];
[educationRubric setGrading:grading];

NSError *error;
NSData *educationRubricData = [educationRubric getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationRubricData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```